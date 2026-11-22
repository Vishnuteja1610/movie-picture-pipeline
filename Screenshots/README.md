# Submission Screenshots Checklist

As described in the project reference guide (Step 6), capture the following screenshots and save them in this `Screenshots/` folder:

1. **`01_github_actions_workflows.png`**:
   - Screenshot of the GitHub repository's **Actions** tab showing successful runs for all 4 workflows:
     - `Frontend Continuous Integration`
     - `Backend Continuous Integration`
     - `Frontend Continuous Deployment`
     - `Backend Continuous Deployment`

2. **`02_frontend_running.png`**:
   - Screenshot of your web browser opening the frontend application at the load balancer URL (e.g. `http://<FRONTEND_LOADBALANCER_URL>`), displaying the **Movie List** catalog fetched from the backend.

3. **`03_backend_api_response.png`**:
   - Screenshot of the browser or terminal (curl) accessing `http://<BACKEND_LOADBALANCER_URL>/movies` showing the JSON response:
     ```json
     {"movies":[{"id":"123","title":"Top Gun: Maverick"},{"id":"456","title":"Sonic the Hedgehog"},{"id":"789","title":"A Quiet Place"}]}
     ```

4. **`04_kubernetes_services.png`**:
   - Screenshot of terminal output running:
     ```bash
     kubectl get services
     kubectl get pods
     kubectl get deployments
     ```

5. **`05_ecr_repositories.png`**:
   - Screenshot of the AWS Console showing the `frontend` and `backend` private ECR repositories with images tagged with git commit SHAs and `latest`.
