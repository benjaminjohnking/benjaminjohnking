# Sandbox Projects

Specifications for common sandbox website and API projects

## Overview

To learn new skills or refine existing skills in a particular technology, a sandbox project should be created and persisted in a dedicated GitHub repository. Sandbox projects may come in two varieties:

1. **Sandbox website** - For front-end technologies
1. **Sandbox API** - For back-end technologies

## Sandbox Website Specifications

Specifications for common sandbox website projects

### Pages

#### Home

- Path: `/`

##### Components

- Headshot
- Personal statement
- Skills
- Links

#### Experience

- Path: `/experience`

##### Components

- List of companies
- Name per company
- List of roles per company
- Title per role
- Start and (if applicable) end dates per role

#### Education

- Path: `/education`

##### Components

- List of credentials
- Degree per credential
- Program per credential
- School per credential
- Start and end dates per credential
- GPA per credential

## Sandbox API Specifications

Specifications for common sandbox API projects

### Endpoints

#### Profile

- Method: `GET`
- Path: `/profile`

##### Schema

```
{
  "image": string,
  "statement": string,
  "links": [
    {
      "title": string,
      "url": string
    }
  ]
}
```

#### Experience

- Method: `GET`
- Path: `/experience`

##### Schema

```
[
  {
    "company": string,
    "roles": [
      {
        "title": string,
        "startDate": string,
        "endDate": string
      }
    ]
  }
]
```

#### Education

- Method: `GET`
- Path: `/education`

##### Schema

```
[
  {
    "degree": string,
    "program": string,
    "school": string,
    "startDate": string,
    "endDate": string,
    "gpa": string"
  }
]
```
