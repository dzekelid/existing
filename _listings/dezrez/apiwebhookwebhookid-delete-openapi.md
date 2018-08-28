---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Deletes an existing webhook.
  version: 1.0.0
  description: Deletes an existing webhook..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/auction/savecontact:
    post:
      summary: Add a new contact to the given auction Role or edit an existing contact
      description: Add a new contact to the given auction role or edit an existing
        contact.
      operationId: Auction_SaveAuctionContactBysaveContactDataContract
      x-api-path-slug: apiauctionsavecontact-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveContactDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Contact
      - To
      - Given
      - Auction
      - Role
      - Edit
      - Existing
      - Contact
  /api/auction/removecontact:
    post:
      summary: Remove an existing auction contact from the auction role
      description: Remove an existing auction contact from the auction role.
      operationId: Auction_RemoveAuctionContactByremoveContactDataContract
      x-api-path-slug: apiauctionremovecontact-post
      parameters:
      - in: body
        name: removeContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Existing
      - Auction
      - Contact
      - From
      - Auction
      - Role
  /api/role/auction/{id}/addtoauction:
    post:
      summary: Add a property auction role to an existing auction
      description: Add a property auction role to an existing auction.
      operationId: AuctionRole_AddToAuctionByidByauctionIdBylotNumber
      x-api-path-slug: apiroleauctionidaddtoauction-post
      parameters:
      - in: query
        name: auctionId
        description: the id of the auction to add the role to
      - in: path
        name: id
        description: the id of the role
      - in: query
        name: lotNumber
        description: the lot number
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Property
      - Auction
      - Role
      - To
      - Existing
      - Auction
  /api/role/auction/{id}/removefromauction:
    post:
      summary: Add a property auction role to an existing auction
      description: Add a property auction role to an existing auction.
      operationId: AuctionRole_RemoveFromAuctionByidByremoveFromAuctionDataContract
      x-api-path-slug: apiroleauctionidremovefromauction-post
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: body
        name: removeFromAuctionDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Property
      - Auction
      - Role
      - To
      - Existing
      - Auction
  /api/cache/List/{listKey}/Append:
    put:
      summary: Adds {itemToAppend} to the tail of an existing list, or creates a new
        list with the object in it.
      description: Adds {itemtoappend} to the tail of an existing list, or creates
        a new list with the object in it..
      operationId: Cache_AppendToListByitemToAppendBylistKeyBytimeToLive
      x-api-path-slug: apicachelistlistkeyappend-put
      parameters:
      - in: body
        name: itemToAppend
        description: The item to append
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - S
      - ItemToAppend
      - To
      - Tail
      - Of
      - Existing
      - List
      - ""
      - Creates
      - New
      - List
      - Object
      - In
      - It
  /api/cache/List/{listKey}/Prepend:
    put:
      summary: Adds {itemToPrepend} to the head of an existing list, or creates a
        new list with the object in it.
      description: Adds {itemtoprepend} to the head of an existing list, or creates
        a new list with the object in it..
      operationId: Cache_PrependToListByitemToPrependBylistKeyBytimeToLive
      x-api-path-slug: apicachelistlistkeyprepend-put
      parameters:
      - in: body
        name: itemToPrepend
        description: The item to prepend
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - S
      - ItemToPrepend
      - To
      - Head
      - Of
      - Existing
      - List
      - ""
      - Creates
      - New
      - List
      - Object
      - In
      - It
  /api/document/setprivacy:
    put:
      summary: Sets the document privacy for an existing document.  This is used to
        change a document from being publicly accessible to being private, and vice
        versa.
      description: Sets the document privacy for an existing document.  this is used
        to change a document from being publicly accessible to being private, and
        vice versa..
      operationId: Document_SetDocumentPrivacyBysetDocumentPrivacyCommand
      x-api-path-slug: apidocumentsetprivacy-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setDocumentPrivacyCommand
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Document
      - Privacyan
      - Existing
      - Document
      - ""
      - ""
      - This
      - Is
      - Used
      - To
      - Change
      - Document
      - From
      - Being
      - Publicly
      - Accessible
      - To
      - Being
      - Private
      - ""
      - Vice
      - Versa
  /api/document/rename:
    put:
      summary: Updates the filename of an existing document.
      description: Updates the filename of an existing document..
      operationId: Document_RenameByrenameDocumentCommandDataContract
      x-api-path-slug: apidocumentrename-put
      parameters:
      - in: body
        name: renameDocumentCommandDataContract
        description: The new filename (excluding the extension)
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Filename
      - Of
      - Existing
      - Document
  /api/group/{id}/addgroupmember:
    put:
      summary: Add a new contact to an existing group
      description: Add a new contact to an existing group.
      operationId: Group_AddGroupMemberByidByaddGroupMemberDataContract
      x-api-path-slug: apigroupidaddgroupmember-put
      parameters:
      - in: body
        name: addGroupMemberDataContract
        description: The details of the person
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - New
      - Contact
      - To
      - Existing
      - Group
  /api/group/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a group
      description: Attaches an existing document to a group.
      operationId: Group_AttachDocumentByidBydocumentId
      x-api-path-slug: apigroupidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the group to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Group
  /api/invoice/{id}/linkfees:
    post:
      summary: Add a fee to an existing invoice
      description: Add a fee to an existing invoice.
      operationId: Invoice_AddLinkedFeesByidByfees
      x-api-path-slug: apiinvoiceidlinkfees-post
      parameters:
      - in: body
        name: fees
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Fee
      - To
      - Existing
      - Invoice
  /api/invoice/{id}/removefee:
    put:
      summary: Remove fee from existing invoice
      description: Remove fee from existing invoice.
      operationId: Invoice_RemoveLinkedFeeByidByattachedFeeId
      x-api-path-slug: apiinvoiceidremovefee-put
      parameters:
      - in: query
        name: attachedFeeId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Fee
      - From
      - Existing
      - Invoice
  /api/invoice/makeallocation:
    post:
      summary: Make an allocation against an existing invoice
      description: Make an allocation against an existing invoice.
      operationId: Invoice_MakeAllocationByallocationDataContract
      x-api-path-slug: apiinvoicemakeallocation-post
      parameters:
      - in: body
        name: allocationDataContract
        description: Details of Allocation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Make
      - Ocation
      - Against
      - Existing
      - Invoice
  /api/milestone/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a milestone
      description: Attaches an existing document to a milestone.
      operationId: Milestone_AttachDocumentByidBydocumentId
      x-api-path-slug: apimilestoneidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the milestone to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Milestone
  /api/progression/savecontact:
    post:
      summary: Add a new contact to the given progression Role or edit an existing
        contact
      description: Add a new contact to the given progression role or edit an existing
        contact.
      operationId: Progression_SaveProgressionContactBysaveContactDataContract
      x-api-path-slug: apiprogressionsavecontact-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveContactDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Contact
      - To
      - Given
      - Progression
      - Role
      - Edit
      - Existing
      - Contact
  /api/progression/removecontact:
    post:
      summary: Remove an existing progression contact from the progression role
      description: Remove an existing progression contact from the progression role.
      operationId: Progression_RemoveProgressionContactByremoveContactDataContract
      x-api-path-slug: apiprogressionremovecontact-post
      parameters:
      - in: body
        name: removeContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Existing
      - Progression
      - Contact
      - From
      - Progression
      - Role
  /api/property/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a property
      description: Attaches an existing document to a property.
      operationId: Property_AttachDocumentByidBydocumentId
      x-api-path-slug: apipropertyidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the property to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Property
  /api/role/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a role
      description: Attaches an existing document to a role.
      operationId: Role_AttachDocumentByidBydocumentId
      x-api-path-slug: apiroleidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the role to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Role
  /api/roomdescription/setimages:
    post:
      summary: Allows you to specify a list of documentIds for a roomDescriptions
        room - this list will overwrite any existing list of documents on that room,
        and order will be honoured.
      description: Allows you to specify a list of documentids for a roomdescriptions
        room - this list will overwrite any existing list of documents on that room,
        and order will be honoured..
      operationId: RoomDescription_SetImagesByroomImageOrder
      x-api-path-slug: apiroomdescriptionsetimages-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: roomImageOrder
        description: The room image order
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Specify
      - List
      - Of
      - DocumentIdsa
      - RoomDescriptions
      - Room
      - '-'
      - This
      - List
      - Will
      - Overwrite
      - Any
      - Existing
      - List
      - Of
      - Documents
      - "On"
      - That
      - Room
      - ""
      - Order
      - Will
      - Be
      - Honoured
  /api/webhook/{webhookId}:
    delete:
      summary: Deletes an existing webhook.
      description: Deletes an existing webhook..
      operationId: Webhook_DeleteWebhookBywebhookId
      x-api-path-slug: apiwebhookwebhookid-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: webhookId
        description: The webhook identifier
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Webhook
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