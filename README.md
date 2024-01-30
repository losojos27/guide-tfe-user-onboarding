# guide-tfe-user-onboarding
Best practices for onboarding users in TFE

The recommended method of onboarding and managing users in Terraform Enterprise is to configure SAML single sign-on (SSO) and enable team membership mapping. This provides the following benefits:
- all the advantages that SSO brings
- no SMTP server configuration in TFE required
- makes the invite process moot and unnecessary

Notes:
It isn't initially clear how to manage org access via SSO. In TFE, the org access is managed via team memberships. When a user is added to a team based on their SAML assertion, they are also added to the org that team belongs to.
