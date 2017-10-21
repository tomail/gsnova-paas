# deploy gsnova-paas to  docker(openshift starter)

gsnova-paas ver 0.29.0

image: wangyi2005/gsnova-paas

# 1.websocket

ServerList: wss://##########.7e14.starter-us-west-2.openshiftapps.com

openshift secure route type: edge(port 8080)

# 2.http2

ServerList: http2://##########.7e14.starter-us-west-2.openshiftapps.com

openshift secure route type: passthrough(port 8088)

# 3.sniproxy setting in client.json and host.json

