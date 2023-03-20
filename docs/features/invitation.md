---
sidebar_position: 2
---

# Invitation

User invites another user to an organization via the endpoint: _"api/organizations/invite/:organizationId"_

When the invitation is sent, an _invite_ record is created in _invites_ table with Organization Id, Invited User Id, and a secret.

Invited user also receives an email with a link to accept or reject the invitation.

When the frontend comes into place, this part will make more sense.

Endpoint to accept the invitation: _/api/organizations/invite/accept_

Endpoint to reject the invitation: _/api/organizations/invite/reject_

Do not forget that _secret_ variable must be send along with these two endpoints.
