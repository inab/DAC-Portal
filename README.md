# Data Access Committee (DAC) Portal

## Summary

This repository contains the DAC-Portal, a key component of the iPC's Data Access Framework where entitled users can create new Data Access Committees, and also, invite other users to join them. The DAC members are able to grant/deny incoming Data Access Requests (DAR) performed by the [iPC's Catalogue](https://github.com/inab/iPC_Data_Portal.git) users, manage user's dataset permissions over time, and also, manage the public information of their respective DACs. Finally, the iPC's Catalogue users can inspect the status of their Data Access Requests directly from the DAC-Portal user interface.

## Architecture

The DAC-Portal is formed by a user interface and a dedicated backend which are divided in two repositories. Both of these repositories are aligned to the Clean Architecture patterns and principles, and more specifically they both follow the Hexagonal Architecture pattern where three layers have been proposed: Domain, Application, and Infrastructure. The system has been designed to be compliant with the Dependency Rule, that can be achieved following the well-known SOLID principles.

A more detailed information about these repositories can be found right below: 

- Backend: [DAC-Portal-backend](https://github.com/inab/DAC-Portal-backend)

- Frontend: [DAC-Portal-frontend](https://github.com/inab/DAC-Portal-frontend)

## Integrations  

- Security: AuthN/Z Keycloak server.

- API's: [Permissions-API](https://github.com/inab/Permissions-API)

- Databases: MongoDB.
