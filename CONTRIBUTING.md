# Contributing to Geniffy

Thank you for helping. This organization holds the parts of Geniffy that run in your code and your tools:
the SDKs, the examples and the MCP server's setup guide. The Geniffy service itself is not developed here.

## Report a bug

Open an issue in the repository it belongs to, with:

- what you did, what you expected, and what happened instead;
- the SDK version, and your Python or Node.js version;
- the request id from the error (`error.request_id` in Python, `error.requestId` in JavaScript), if there
  is one. It lets us find that exact call.

Never paste an API key into an issue. If you did, revoke it in the Geniffy app under **API keys**.

For a security problem, follow the [security policy](SECURITY.md) instead.

## Suggest a change

For anything bigger than a small fix, open an issue first, so we can agree on the approach before you
spend time on it.

## Send a pull request

1. Fork the repository and create a branch.
2. Make the change, with a test when it changes behaviour.
3. Run the tests:
   - Python SDK: `pip install -e ".[test]"`, then `pytest`
   - TypeScript SDK: `npm ci`, then `npm test`
4. Open the pull request, and say what changed and why.

By sending a pull request, you agree that your contribution is licensed under the repository's license (MIT).
