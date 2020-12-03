# gcp-gae-delivery

## Initial Setup

```bash
make install
gcloud projects describe $GOOGLE_CLOUD_PROJECT
gcloud config set project $GOOGLE_CLOUD_PROJECT
```

## Create Google App Engine

```bash
gcloud app create
```

## Deploy the app

```bash
gcloud app deploy
```

The app is deployed at this [link](https://gcp-gae-delivery.ey.r.appspot.com).

## Stream logs

```bash
gcloud app logs tail -s default
```

## Automating App Engine Deployment

[Reference](https://cloud.google.com/source-repositories/docs/quickstart-triggering-builds-with-source-repositories).

Follow the steps from ref.
- Enable the APIs.
- Grant App Engine access to the Cloud Build service account.
  - Enable App Engine
  - Enable Service account
