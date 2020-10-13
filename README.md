
# Magic Lambda Image

Image manipulation library for Magic, allowing you to do basic manipulation of images, in addition to generating
QR codes.

## Generating a QR code

You can use the **[qr.generate]** slot to create a QR code. This slow returns the QR code as a `MemoryStream`, which
allows you to return its output directly over the HTTP response object, which again will persist the QR code
back as the response to the caller if you're in a web project of some sort using Magic. The slot takes two arguments.

* Value of node - Mandatory string to become the content of the generated QR code
* __[size]__ - Optional argument declaring the size of your QR code

Below is an example of usage

```
qr.generate:"https://reddit.com"
   size:8
```

After execution, the above invocation slot will contain a `MemoryStream` encapsulating your underlaying code.

## Quality gates

- [![Build status](https://travis-ci.com/polterguy/magic.lambda.image.svg?master)](https://travis-ci.com/polterguy/magic.lambda.image)
- [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=alert_status)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=bugs)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=code_smells)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=coverage)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=duplicated_lines_density)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=ncloc)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=security_rating)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=sqale_index)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
- [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=polterguy_magic.lambda.image&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=polterguy_magic.lambda.image)
