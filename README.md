if we use different data type into configmap
----- kubectl get configmap jot-config -o yaml

if we use single line output from different data type
 -----kubectl get secret my-secret -o jsonpath='{.data.string-value}' | base64 -d
 -----kubectl get secret my-secret -o jsonpath='{.data.yaml-value}' | base64 -d
