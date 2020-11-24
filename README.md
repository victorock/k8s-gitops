GitOps of K8S resources.

Folder Structure:

- ansible-control
        - awx-operator.yml  
          `-> Control-Plane Execution Environment
        - awx-resource-operator.yml  
          `-> Control-plane Configuration  
        - argocd-operator.yml  
          `-> Control-Plane Configuration Policy  
        - gitea-operator.yml  
          `-> Control-Plane Configuration Store  

- ansible-data
    - deploy
        - galaxy-operator.yml  
          `-> Content Distribution
        - gitea-operator.yml  
          `-> Content Store

- ansible-monitor
    - deploy
        - grafana-operator.yml  
          `-> Visualization & Reporting
        - elastic-operator.yml  
          `-> Datastore (Logging, Facts, etc...)
        - prometheus-operator.yml  
          `-> Telemetry & Alert Management
        - prometheus-exporter-operator.yml  
          `-> Telemetry Collector
