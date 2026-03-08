# Multi-stage build - Production ready Docker image
FROM python:3.11-slim

# Set working directory
WORKDIR /app

# Copy the webapp files
COPY index.html .
COPY style.css .
COPY script.js .
COPY server.py .

# Create a non-root user for security
RUN useradd -m -u 1000 webapp && chown -R webapp:webapp /app

# Switch to non-root user
USER webapp

# Expose port
EXPOSE 8000

# Health check
HEALTHCHECK --interval=30s --timeout=10s --start-period=5s --retries=3 \
    CMD python -c "import urllib.request; urllib.request.urlopen('http://localhost:8000')" || exit 1

# Run the server
CMD ["python", "server.py"]
