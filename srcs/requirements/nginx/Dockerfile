FROM alpine:3.20
# No cache because we don't need them and I HAVE LIMITED DRIVE
RUN	apk update && apk upgrade && apk add --no-cache nginx
# Exposing the 443 ofc, why ? SUBJECT RULES
EXPOSE 443
# Run the nginx itself in daemon off (dont run in BG) to get the all the logs in the terminal of container 
CMD ["nginx", "-g", "daemon off;"]
