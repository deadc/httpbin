# httpbin

Sample app

# sleep

    export SLEEP_POD=$(kubectl get pod -l app=sleep -o jsonpath={.items..metadata.name})
    kubectl exec -it $SLEEP_POD -c sleep -- curl http://endpoint:port/uri
