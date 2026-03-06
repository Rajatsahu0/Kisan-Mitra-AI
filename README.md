# Kisan Mitra AI

A unified professional-grade rural innovation platform that integrates voice, vision, and data analytics to support farmers through the entire agricultural lifecycle.

## Project Structure

```
KisanMitraAI/
├── src/
│   ├── KisanMitraAI.API/          # ASP.NET Core Web API & CoreWCF SOAP services
│   ├── KisanMitraAI.Core/         # Domain models, interfaces, business logic
│   └── KisanMitraAI.Infrastructure/ # AWS SDK integrations, data access, external services
├── tests/
│   └── KisanMitraAI.Tests/        # Unit tests and property-based tests (FsCheck)
└── KisanMitraAI.sln               # Solution file
```

## Technology Stack

- **.NET 8**: Modern, high-performance framework
- **AWS AI Services**: Transcribe, Bedrock (Claude 3.5 Sonnet), Rekognition, Textract, Polly
- **AWS Infrastructure**: S3, DynamoDB, Timestream, Step Functions
- **Database**: PostgreSQL with Entity Framework Core
- **SOAP Integration**: CoreWCF for government system integration
- **Testing**: xUnit with FsCheck for property-based testing

## Core Modules

1. **Krishi-Vani**: Voice-first market intelligence with regional dialect support
2. **Quality Grader**: Vision-based produce grading using AI
3. **Dhara-Analyzer**: Soil health card digitization and regenerative farming plans
4. **Sowing Oracle**: Predictive planting recommendations

## Getting Started

### Prerequisites

- .NET 8 SDK
- AWS Account with configured credentials
- PostgreSQL database
- Visual Studio 2022 or VS Code

### Configuration

Update `src/KisanMitraAI.API/appsettings.json` with your AWS credentials and service endpoints.

### Build

```bash
dotnet build
```

### Run Tests

```bash
dotnet test
```

### Run API

```bash
dotnet run --project src/KisanMitraAI.API
```

## AWS Services Configuration

The platform requires the following AWS services to be configured:
- Amazon Transcribe (voice-to-text)
- Amazon Bedrock (LLM for query parsing and response generation)
- Amazon Rekognition (image analysis)
- Amazon Textract (document OCR)
- Amazon Polly (text-to-speech)
- Amazon S3 (object storage)
- Amazon DynamoDB (NoSQL database)
- Amazon Timestream (time-series database)
- AWS Step Functions (workflow orchestration)
- Amazon Cognito (authentication)

## License

Copyright © 2026 Kisan Mitra AI Team
