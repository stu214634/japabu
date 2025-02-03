# Use multi-architecture Alpine image explicitly
FROM --platform=linux/arm64 nginx:alpine

# Set platform arguments (useful for multi-arch builds)
ARG TARGETARCH
ARG TARGETPLATFORM

# Install any required dependencies (if needed)
# RUN apk add --no-cache [any-arm64-compatible-packages]

# Copy web content
COPY index.html /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start server
CMD ["nginx", "-g", "daemon off;"]