
# gRPC Invoicer Service


This link is the inspiration. Shout out to the creator of this video. 
[Youtube](https://www.youtube.com/watch?v=gbrPMv_GuQY)

---
This is a simple gRPC service written in Go that provides two endpoints for creating and updating invoices.

## Overview

The service implements the following RPC methods:
- `Create`: Generates a response with PDF and Docx files based on the `CreateRequest`.
- `Update`: Updates an invoice and returns updated files.

## Prerequisites

- Go 1.18+
- gRPC and Protobuf support for Go.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo-url
   cd gRPC_golang
   ```

2. Install dependencies:

   ```bash
   go mod tidy
   ```

## Running the Service

To start the gRPC server:

```bash
go run main.go
```

The server will listen on `localhost:8089`.

## gRPC API

### Create

- **Request**: `CreateRequest`
    - `From` (string): A required field for invoice creation.

- **Response**: `CreateResponse`
    - `Pdf`: A byte array of the generated PDF.
    - `Docx`: A byte array of the generated Docx file.

### Update

- **Request**: `CreateRequest`
    - `From` (string): Invoice data to be updated.

- **Response**: `CreateResponse`
    - `Pdf`: A byte array of the updated PDF.
    - `Docx`: A byte array of the updated Docx file.

## License

This project is licensed under the MIT License.

---

