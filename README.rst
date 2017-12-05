gvl-galaxy-release-test-workflows
=================================
A set of workflows that are used to check that Galaxy is running correctly prior to a release of the GVL

Installation
~~~~~~~~~~~~
Install the latest release from PyPi:

.. code-block:: shell

  git clone https://github.com/gvlproject/gvl-galaxy-release-test-workflows
  cd gvl-galaxy-release-test-workflows
  virtualenv --prompt "(gvl-release-test-workflows)" -p python3 venv
  source venv/bin/activate
  pip install -r requirements.txt


Running tests
~~~~~~~~~~~~~
To run a workflow

.. code-block:: shell

  export GALAXY_URL=<galaxy_server_url>
  export GALAXY_API_KEY=<galaxy_api_key>
  wft4galaxy -f galaxy-101/workflow-test-suite.yml

To generate a test
~~~~~~~~~~~~~~~~~~

http://wft4galaxy.readthedocs.io/