## prometheus
use the command below to run docker compose file
```bash
docker-compose up
```

Jenkins Prometheus Metrics Plugin:

It will expose the Jenkins metrics in Prometheus.

To install this plugin,
Login to Jenkins > manage jenkins > manage plugins >  Available > then search for "Prometheus metrics plugin"  then install it.
Now after installation we need to configure the Prometheus details in Jenkins.
Login to Jenkins > manage Jenkins > Configure Systems > Go to Prometheus section to fill the details like below,

![prom jenkins plugin](https://github.com/xxSURIxx/prometheus/assets/143709408/b7840cd0-fca8-4408-a245-e0059acf4ba7)
Then save the configuration.


Next we need to configure Prometheus in Grafana data-sources.
Login to Grafana > Go to configuration > Choose data source > Add data source > select Prometheus > Enter the Prometheus server details,

![prometheus server detais](https://github.com/xxSURIxx/prometheus/assets/143709408/0304befd-6379-415e-bc70-b647409fd340)

Once given the details click "Save & Test", it should say Data Source is working like below image,

Dashboard

![prom_ser_conf](https://github.com/xxSURIxx/prometheus/assets/143709408/e2721cef-d441-4be2-8637-01227b6a9735)

![Screenshot from 2023-11-29 12-05-06](https://github.com/xxSURIxx/prometheus/assets/143709408/60fc382e-d5cf-4166-adee-e9a4aee74fbd)
![Screenshot from 2023-11-29 12-05-42](https://github.com/xxSURIxx/prometheus/assets/143709408/fd558bff-8749-433b-9685-b9f684456f7b)

