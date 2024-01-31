# innov_week
centering my innovation week projects around here!

## jan24 [ K8sGPT: powering kubernetes with AI ]
Hey, this innovation week presentation focus on the usage of K8sGPT, an AI based tool that scan your cluster, looks for issues and vulnerabilities and recommends solutions!

 * __step 1:__ _Install the helm chart of K8sGPT_
 ```shell
helm repo add k8sgpt https://charts.k8sgpt.ai/ #add repo
helm repo update # update repos
helm install release k8sgpt/k8sgpt-operator -n k8sgpt-operator-system --create-namespace #install helm chart
 ```

 > __PS:__ There is a CLI version as well, but considering that the helm version restricts the tool within the deployed and target clusters, it seemed a safer option for tool that is still in development


 * __step2__: _Create your OPEN AI API KEY_<br>

&emsp;&emsp;&emsp; Go to OPEN AI website, log in.<br>
&emsp;&emsp;&emsp; Select the API key section in the menu and create an API key.<br>
&emsp;&emsp;&emsp; Copy it!