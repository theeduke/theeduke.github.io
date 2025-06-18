---
title: "Carpooling Webapp"
permalink: /projects/carpooling-webapp/
layout: single
author_profile: true
excerpt: "A web application for ride-sharing in Nairobi, built with React, Django, and Google Maps API."
header:
  image: /assets/images/carpooling-thumbnail.jpg
  teaser: /assets/images/carpooling-teaser.jpg
classes: wide
gallery:
  - url: /assets/images/carpooling-screenshot1.jpg
    image_path: /assets/images/carpooling-screenshot1.jpg
    alt: "Carpooling App Screenshot 1"
  - url: /assets/images/carpooling-screenshot2.jpg
    image_path: /assets/images/carpooling-screenshot2.jpg
    alt: "Carpooling App Screenshot 2"
---

## Overview
A web application for ride-sharing in Nairobi, featuring secure authentication, real-time ride search, and in-app payments.

**Tech Stack**: React, Django, Django REST Framework, Google Maps API, PostgreSQL  
**Contributions**: Developed backend APIs, implemented route optimization, and integrated payment systems.  
**Links**:  
- [GitHub](https://github.com/theeduke/carpooling-webapp)  
- [Live Demo](https://example.com/carpooling) *(replace with actual link if available)*  

## Key Features
- **Secure Authentication**: Implemented JWT-based authentication for user login.
- **Real-Time Ride Search**: Integrated Google Maps API for location-based ride matching.
- **In-App Payments**: Added Stripe for secure payment processing.

## Code Snippet
Example of a Django view for ride search:
```python
from rest_framework.views import APIView
from rest_framework.response import Response
from .models import Ride
from .serializers import RideSerializer

class RideSearchView(APIView):
    def get(self, request):
        location = request.query_params.get('location')
        rides = Ride.objects.filter(start_location__near=location)
        serializer = RideSerializer(rides, many=True)
        return Response(serializer.data)
