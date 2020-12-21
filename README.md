# Octopus Deploy Release Action
A Simple Action that uses the Octopus Deploy [`octo`](https://hub.docker.com/r/octopusdeploy/octo) Docker Image to Create a new Release for a given Project

## Inputs

### `server`

**Required** The URI of your Octopus Deploy Instance

### `apiKey`

**Required** The API Key used to Authenticate with Octopus Deploy

### `project`

**Required** The Name of the Project for this new Release

### `version`

**Required** The Version for this Release

## Example Usage

```yml
uses: ricado-group/octopus-deploy-release-action@v1.0.0
with:
  server: 'https://instancename.octopus.app'
  apiKey: ${{ secrets.OCTOPUS_APIKEY }}
  project: 'MyProjectName'
  version: '2.1.0'
```