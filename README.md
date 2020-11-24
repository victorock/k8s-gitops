GitOps of K8S resources.

Folder Structure:

- ansible-control
    - deploy
        - awx-operator.yml
          `-> Control-Plane
        - awx-resource-operator.yml
          `-> Control-plane Configuration

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
