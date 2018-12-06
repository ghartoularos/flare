# Set up a virtualenv to house the requirements
virtualenv flare.process

# Then activate it
source flare.process/bin/activate

# Now that its activate, install the packages from the requirements file. This includes ipykernel, which is used to set up a jupyter kernel that sources this environments packages.
flare.process/bin/pip install -r requirements.txt

# Then install the new kernel
ipython kernel install --user --name=flare.process

# Now you can launch jupyter notebook, and open the notebook with the kernel you just created, and the notebook should (hopefully) run smoothly.
