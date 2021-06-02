## How to run the kuttl tests
1. Create a namespace in your cluster called 'test-project' (this needs to match what is in kuttl-test.yaml)
1. Ensure you are logged into your cluster and test-project is the current namespace
1. Install the CRDs into the namespace with 'make install-all'
1. Ensure you have operator SDK 0.15.2 installed
1. Run the controller locally with 'operator-sdk run --local'
1. Ensure you have the kuttl plugin for kubectl installed correctly
1. Run 'kubectl kuttl test ./test/il'
