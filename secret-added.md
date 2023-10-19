# Added a secret

Used the following command to add a secret to be accessed by the `dags/example_dag.py` file:

```bash
gcloud config set project qwiklabs-gcp-02-45f2a83d398e
echo -n "eric test secret" | gcloud secrets create example-variables-eric_secret --replication-policy="automatic" --data-file=-
```

This is then accessable at: `var.value.eric_secret`.