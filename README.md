# KubeWharf Website

Welcome to the GitHub repository for KubeWharf's public website!

The docs website is hosted at https://kubewharf.github.io.

We use [Hugo](https://gohugo.io/) with the [google/docsy](https://github.com/google/docsy)
theme for styling and site structure.

## Quicistart
Here's a quick guide to updating the repo:
1. download repo
    ```bash
    git clone --depth 1 https://github.com/kubewharf/github.io
    ```
1. (Optional) If you want to do SCSS edits and want to publish these, you need to install `PostCSS`
    ```bash
    npm install
    ```

## Running a container locally (recommended)

You can run docsy-example inside a [Docker](https://docs.docker.com/)
container, the container runs with a volume bound to the `docsy-example`
folder. This approach doesn't require you to install any dependencies other
than [Docker Desktop](https://www.docker.com/products/docker-desktop) on
Windows and Mac, and [Docker Compose](https://docs.docker.com/compose/install/)
on Linux.

1. Build the docker image 

   ```bash
   docker-compose build
   ```

1. Run the built image

   ```bash
   docker-compose up
   ```

   > NOTE: You can run both commands at once with `docker-compose up --build`.

1. Verify that the service is working. 

   Open your web browser and type `http://localhost:1313` in your navigation bar,
   This opens a local instance of the kubewharf homepage. You can now make
   changes to the code and those changes will immediately show up in your
   browser after you save.

### Cleanup

To stop Docker Compose, on your terminal window, press **Ctrl + C**. 
To remove the produced images run:
    
    docker-compose rm
    

## Running the website locally

Building and running the site locally requires a recent `extended` version of [Hugo](https://gohugo.io).
You can find out more about how to install Hugo for your environment in
[Getting started](https://www.docsy.dev/docs/getting-started/#prerequisites-and-installation) guide.

Once you've made your working copy of the site repo, from the repo root folder, run:

```
hugo server
```


## Community

Email: kubewharf.conduct@bytedance.com

## License
This project is licensed under the [Apache-2.0 License](LICENSE).
