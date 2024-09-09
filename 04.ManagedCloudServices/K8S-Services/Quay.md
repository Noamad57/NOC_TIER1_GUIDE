# Quay


#### Getting Started 
- [ ] Get familiar with the concept of docker images 
- [ ] Get familiar with image management tools (docker, podman).

#### Basic Questions

1. What is an image registry? give some examples.
2. What is Quay?
3. Why do you need an image registry?
4. What are some feaures of Quay?
5. Explain these Quay concepts:
     1. Organization
     2. Repository
     3. Tag
      4. Time machine
     5. Quota
6. Explain about the permmissions structure in Quay
      1. Team
     2. Default permissions
     3. Team role
     4. Repository permissions
7. What is a robot account?
8. What are private repositories? How do you set a repository as public?
9. How would you use images from private repositories in an OpenShift pod?
10. What are image tag and digest?
11. Push an untagged image to Quay, what happend?
12. What happens to a tag after you delete it? How do you delete it from the time machine?
13. How do you authenticate to the Quay's api?


## Task

###### Pre-Requirements
Ask your trainee to prepare for you:  
- [ ] OpenShift namespace
- [ ] Organization in Quay

###### The task
1. Build a docker image that has your favorite cli in it 
2. Push the image to your Quay organization 
3. Ensure that the repository of your image is private
4. Create a deployment in OpenShift that uses your image 
5. Configure tag expiration on your image, so it would be deleted in 3 days
 
