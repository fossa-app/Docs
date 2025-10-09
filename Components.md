
| Component                                                           | Aspect            | Docker Image                         | Tech Stack                                                     |
| ------------------------------------------------------------------- | ----------------- | ------------------------------------ | -------------------------------------------------------------- |
| [FusionAuth](https://fusionauth.io/)                                | Identity Provider | fusionauth/fusionauth-app            | - PostgreSQL relational database<br>- Elasticsearch (Optional) |
| [API](https://github.com/fossa-app/API)                             | Backend API       | tiksn/fossa-api                      | [ASP.NET Core](https://asp.net/)                               |
| [UI](https://github.com/fossa-app/UI)                               | Frontend SPA      | tiksn/fossa-ui                       | [React](https://react.dev/)                                    |
| [OpenTelemetry Collector](https://opentelemetry.io/docs/collector/) | Observability     | otel/opentelemetry-collector-contrib | -                                                              |
| [MongoDB](https://www.mongodb.com/)                                 | Primary Database  |                                      | -                                                              |
