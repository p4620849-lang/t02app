Project 2 Rationale

Base Image

I selected nginx:alpine as the final image because it is lightweight and efficient for serving static web content. Using a multi-stage Docker build removes unnecessary development tools from the final image and reduces image size.

Service Split

I used separate web and cache services. The web service provides application content, while Redis provides caching. Using separate services follows container best practices because each service has a single responsibility and can be managed independently.