---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Returns a list of email templates associated to this agency
  version: 1.0.0
  description: Returns a list of email templates associated to this agency.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accountingsystem/officeaccounts:
    get:
      summary: Get list of office accounts associated with the accounting system
      description: Get list of office accounts associated with the accounting system.
      operationId: AccountingSystem_GetOfficeAccounts
      x-api-path-slug: apiaccountingsystemofficeaccounts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Office
      - Accounts
      - Associated
      - Accounting
      - System
  /api/documentgeneration/lettertemplate/{letterTemplateId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetLetterTemplateByletterTemplateId
      x-api-path-slug: apidocumentgenerationlettertemplatelettertemplateid-get
      parameters:
      - in: path
        name: letterTemplateId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/mergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetPrintableMergeTemplates
      x-api-path-slug: apidocumentgenerationmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/unusedmergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency that are
        not currently used in any envelope templates
      description: Returns a list of lettertemplates associated to this agency that
        are not currently used in any envelope templates.
      operationId: DocumentGeneration_GetUnusedMergeTemplates
      x-api-path-slug: apidocumentgenerationunusedmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - That
      - Are
      - Not
      - Currently
      - Used
      - In
      - Any
      - Envelope
      - Templates
  /api/documentgeneration/templatesusinganalytics/{analyticsId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency and to
        a particular google analyitics campaign
      description: Returns a list of lettertemplates associated to this agency and
        to a particular google analyitics campaign.
      operationId: DocumentGeneration_GetTemplatesUsingAnalyticsByanalyticsId
      x-api-path-slug: apidocumentgenerationtemplatesusinganalyticsanalyticsid-get
      parameters:
      - in: path
        name: analyticsId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - To
      - Particular
      - Google
      - Analyitics
      - Campaign
  /api/documentgeneration/insertabletemplates:
    get:
      summary: Returns a list of insertable templates associated to this agency
      description: Returns a list of insertable templates associated to this agency.
      operationId: DocumentGeneration_GetPrintableInsertableTemplates
      x-api-path-slug: apidocumentgenerationinsertabletemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Insertable
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/headertemplates:
    get:
      summary: Returns a list of header templates associated to this agency with their
        associated brand info
      description: Returns a list of header templates associated to this agency with
        their associated brand info.
      operationId: DocumentGeneration_GetPrintableHeaderTemplates
      x-api-path-slug: apidocumentgenerationheadertemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Header
      - Templates
      - Associated
      - To
      - This
      - Agency
      - Their
      - Associated
      - Brand
      - Info
  /api/documentgeneration/envelopetemplates:
    get:
      summary: Returns a list of envelope templates associated to this agency
      description: Returns a list of envelope templates associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplates
      x-api-path-slug: apidocumentgenerationenvelopetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacks:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePacks
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacks-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacktypes:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackTypesByinUseOnly
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacktypes-get
      parameters:
      - in: query
        name: inUseOnly
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/emailtemplates:
    get:
      summary: Returns a list of email templates associated to this agency
      description: Returns a list of email templates associated to this agency.
      operationId: DocumentGeneration_GetEmailTemplates
      x-api-path-slug: apidocumentgenerationemailtemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Email
      - Templates
      - Associated
      - To
      - This
      - Agency
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---