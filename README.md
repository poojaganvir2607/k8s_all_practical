all k8s practical
amivir@Amits-MacBook-Air k8s % kubectl get cronjob
NAME         SCHEDULE      TIMEZONE   SUSPEND   ACTIVE   LAST SCHEDULE   AGE
my-cronjob   */5 * * * *   <none>     False     0        88s             9m33s
amivir@Amits-MacBook-Air k8s % kubectl get job
NAME                  STATUS     COMPLETIONS   DURATION   AGE
my-cronjob-29271135   Complete   1/1           20s        6m38s
my-cronjob-29271140   Complete   1/1           29s        98s
amitganvir@Amits-MacBook-Air k8s % kubectl describe cronjob my-cronjob
Name:                          my-cronjob
Namespace:                     default
Labels:                        <none>

