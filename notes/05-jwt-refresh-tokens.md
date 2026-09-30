# JWT Refresh Token Rotation

Rotate refresh tokens on every use and store only their hash server-side. If a used-and-rotated token is presented again, treat it as a signal of theft and revoke the whole token family.
