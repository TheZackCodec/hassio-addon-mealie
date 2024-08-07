# Use the official Mealie Docker image
FROM ghcr.io/mealie-recipes/mealie:latest

# Set environment variables necessary for Ingress
ENV INGRESS=true

# Expose the application port
EXPOSE 9000

# Start Mealie application
CMD ["gunicorn", "--bind", "0.0.0.0:9000", "mealie.__main__:create_app()"]
