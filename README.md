import dagshub
dagshub.init(repo_owner='fauxcadet', repo_name='ML_Flow_Project', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)