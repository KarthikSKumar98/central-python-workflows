# central-python-workflows
> [!NOTE]
> If you’re looking for Classic Central workflows, please click [here](/Classic-Central/)

This repository contains Python-based workflows, code samples, and where applicable, Postman collections to help automate and integrate with New Central and HPE GreenLake Platform (GLP) APIs.
It leverages the [pycentral SDK](https://pypi.org/project/pycentral/) to interact with Central’s APIs and extensibility features.

Each folder represents a self-contained workflow. Inside each, you’ll find:
- A dedicated README.md explaining the purpose and usage of the workflow
- All required scripts, data files (like CSVs), and Postman collections (if applicable)
- Clear setup and execution instructions

## New Central Workflows
> [!CAUTION]
> The workflows in this section use pre-release versions of the **pycentral** library and are intended primarily for New Central, currently in Public Preview.
> Please note:
> - APIs and SDK behavior may change as the new Central platform evolves with each release.
> - Some workflows may break or require updates with future SDK changes.\
> 
>We will make every effort to keep these workflows up to date. If you encounter any issues or inconsistencies, please open an issue in this repository.

- **[Onboarding](/device-onboarding/)** — Takes factory-default devices from unassigned in GLP through application and subscription assignment, then site, persona, and group setup in New Central.
- **[Ping and iPerf Troubleshooting Workflow](/troubleshooting-workflow/)** — Runs ping and iPerf bandwidth tests from gateways to check connectivity and network performance.
- **[Tunnelled SSID Workflow](/tunneled-ssid-overlay/)** — Creates the roles, policies, overlay WLAN profiles, and tunnelled SSID, assigns them to scopes, and moves devices into sites.
- **[Open SSID Workflow](/open-ssid-overlay/)** — Creates the roles, policies, and an Open (OWE) SSID, assigns them to scopes, and moves devices into the site so they inherit it.
- **[WPA3 PSK Workflow](/wpa3-psk-overlay/)** — Creates the roles, policies, and a WPA3 PSK SSID, assigns them to scopes, and moves devices into the site so they inherit it.
- **[Hierarchy Visualizer](/hierarchy-visualizer/)** — Maps the Central hierarchy and its scope attributes into a terminal summary, a CSV report, and diagrams.
- **[Client Disconnection](/client-disconnect/)** — Finds active clients by MAC address and disconnects them from the device they are connected to.
- **[Rename Hostnames](/rename-hostnames/)** — Renames devices in bulk from a CSV of serial numbers and new hostnames.
- **[Profile Operations](/profile-operations/)** — Shows how to connect with the pycentral base object and run individual and bulk profile operations.
- **[Device Metrics Export](/device-metrics-export)** — Combines device attributes, monitoring data, connectivity, and subscription details from Central and GLP into one CSV.
- **[Cutover Validation](/cutover-validation)** — Runs a set of troubleshooting show commands across online devices and exports the results as HTML, Markdown, or JSON.
- **[MSP Workbench](/msp-workbench/)** — A guided web app and CLI for MSPs, using one MSP credential. Onboard: create tenants, add devices to the MSP inventory, and assign devices and subscriptions to tenants. Observe: monitor tenants and track subscription burndown.

## HPE Greenlake Platform Workflows

- **[Onboarding](/glp-device-onboarding/)** — Assigns devices to an application and applies subscriptions to them, with a matching [Postman collection](/glp-device-onboarding/Postman-Collection/).

## Classic Central Workflows
- [Device Provisioning](/Classic-Central/device_provisioning/)
- [Device Onboarding](/Classic-Central/device_onboarding/)
- [MSP Customer Onboarding](/Classic-Central/msp_customer_onboarding/)
- [MSP Customer Deletion](/Classic-Central/msp_customer_deletion/)
- [Inventory to Excel Workflows](/Classic-Central/inventory_to_excel/)
- [AP CLI Workflows](/Classic-Central/ap_config/)
- [WLAN Workflows](/Classic-Central/wlan_config/)
- [Detailed Central Device Inventory](/Classic-Central/detailed_central_device_inventory/)
- [Device Inventory Migration](/Classic-Central/device_inventory_migration/)
- [User Provisioning](/Classic-Central/user_provisioning/)
- [Bulk Renaming of APs (with CSV)](/Classic-Central/renaming_aps/)
- [Connected Clients](/Classic-Central/connected_clients/)
- [Classic Central Postman Collection](https://www.postman.com/hpe-aruba-networking/workspace/hpe-aruba-networking-central/overview)
- [Streaming API Websocket Client Application](/Classic-Central/streaming-api-client/)
- [Webhook Client application](/Classic-Central/webhooks/)
