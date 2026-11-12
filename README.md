# Over-Engineered Simple Calculator - Instance Version

Backend of the Over-Engineered Simple Calculator that runs the shared calculator core on virtual machine instances with automatic scaling.

- The cloud-agnostic business core lives in `core/`.
- Each cloud has its own isolated root: `aws/` (Amazon EC2 Auto Scaling, AWS SAM) and `azure/` (reserved for a future replica on Virtual Machine Scale Sets).
- The API keeps the same contract as the other backends of the project under `/api/v1`, plus its own prefix `/api/instance/v1`; every response identifies the backend as `instance`.

Status: under construction. Product documentation will be in `docs/`; planned follow-up work is listed in [docs/improvement-backlog.md](docs/improvement-backlog.md).
