Use `build_gpu_docker.sh` to build a docker image. 

Once inside the docker container (using docker run), run the following commands:

`git clone https://github.com/anmakon/meshpy.git`
`cd meshpy`

At this point, edit the setup.py file requirements and change `sklearn` to `scikit-learn==0.20.4`. Then run the rest of the commands:

`python setup.py develop`
`cd ../dex-net`
`python setup.py develop`

From the docker container, run `test/grasping_test.py` for grasping unit tests.
