# Feedback on Avail Node Documentation

## Document Reference
- **Section**: [Running a Full Node](https://docs.availproject.org/docs/operate-a-node/run-a-full-node/full-node)

## Feedback Summary
When attempting to run an Avail node using Docker as per the documentation, the provided command does not successfully locate or pull the Docker image `availj/avail:2.2.4.1`.

## Issue Description
Upon running the command:
```bash
docker run --restart=on-failure -d -v /root/avail/node-data:/da/node-data -p 9944:9944 -p 30333:30333 docker.io/availj/avail:2.2.4.1 --chain mainnet -d ./output --name a-random-name
```
The following error occurs
```bash
Unable to find image 'availj/avail:2.2.4.1' locally
docker: Error response from daemon: failed to resolve reference "docker.io/availj/avail:2.2.4.1": docker.io/availj/avail:2.2.4.1: not found.
```

## Screenshot of the command Running

<img width="1361" alt="Screenshot 2024-10-29 at 1 44 24 AM" src="https://github.com/user-attachments/assets/166b2fad-d78c-4c11-a026-9e277ffc54bd">

## Screenshot of Docker Pull Error for availj/avail:v2.2.4.1 Image Locally

 ![WhatsApp Image 2024-10-30 at 23 23 20](https://github.com/user-attachments/assets/9f90bf30-9b20-4b3a-9757-94b79a776eed)


## Suggested Improvement
1. **Confirm Image Availability**: Ensure that `availj/avail:2.2.4.1` is publicly available on Docker Hub or provide an alternative link or tag in the documentation.
2. **Add Troubleshooting Instructions**: If this image requires specific credentials or access permissions, consider adding a troubleshooting section that covers:
   - How to check for the latest image tag.
   - Steps to authenticate if the image is restricted.
   - Common Docker errors related to image retrieval.

## Additional Comments
Adding these details could improve the onboarding experience for developers and reduce setup issues related to Docker image access.
