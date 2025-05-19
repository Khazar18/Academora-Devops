# Serve the pre-built frontend
FROM node:20-alpine

# Install serve globally to serve the build
RUN npm install -g serve

# Set working directory
WORKDIR /app

# Copy the local pre-built dist directory into the container
COPY dist ./dist

# Set environment and expose port
ENV PORT=5000
EXPOSE 5000

# Run the app with serve
CMD ["serve", "-s", "dist", "-l", "5000"]