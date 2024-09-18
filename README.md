# basic-kserve-vllm

1. Create minio and your data connections using the setup/setup-s3.yaml.
   ```shell
   kubectl apply -n my-namespace -f setup/setup-s3.yaml 
   ```

2. Start a workbench using with git-lfs installed.  OpenShift AI PyTorch notebook will work well.  Make sure to set the data connection to `My Storage`

3. Clone this repository and run the notebook [1_download_save.ipynb](1_download_save.ipynb)

4. Serve a model using the UI or apply the yaml from [sample-deployments](sample-deployments)

5. Test out the new endpoint using [2_vllm_rest_requests.ipynb](2_vllm_rest_requests.ipynb) and [3_vllm_openai_requests.ipynb](3_vllm_openai_requests.ipynb)
