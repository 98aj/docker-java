# This is simple java class printing Hello world in Docker container.
  1. To run this class we used docker file for createing container that have java environment to run this java file
  2. In this docker file we have used jdk image form amazoncorretto 17 alpine version (FROM amazoncorretto:17-alpine)
  3. Workdir is creating working directory in container for java app
  4. COPY . /app ==> is used to copy code form current directory of host to container
  5. RUN => compile the java code
  6. CMD => runs the java file
  7. To build this docker images => docker build -t java-app .
  8. To run container with above created images ==> docker run --name java-docker-cont java-app
