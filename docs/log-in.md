# Log in and launch a session

## Log in

1. Go to <https://jupyter-health.2i2c.cloud> and click {guilabel}`Log in to continue`.

   ```{figure} images/hub-login.png
   :alt: The hub landing page with a Log in to continue button
   :width: 500px
   ```

2. You are sent to the JupyterHealth Exchange.
   Enter the email address and password of your exchange account and click {guilabel}`Log In`.

   ```{figure} images/exchange-login.png
   :alt: The JupyterHealth Exchange log in form
   :width: 300px
   ```

3. You are sent back to the hub, which starts your server.

% We need a more user-friendly documentation of organizations in JHE!
Access is granted by membership in a [JupyterHealth Exchange organization](xref:jhe/jhe/access-control#organization-hierarchy-and-authority).
If you don't have an account, use {guilabel}`Sign Up` on the exchange log in form, then ask your study or organization administrator to add you to their organization.

:::{note}
% We need a more user-friendly documentation of organizations in JHE!
If you get an error after logging in, you are probably not in an organization yet.
See the [exchange access control docs](xref:jhe/jhe/access-control) for how accounts, roles, and organizations work.
:::

## Launch a session

After you log in, the hub starts a JupyterLab server for you.
It might take a minute or two!

## User environment

The server runs the [JupyterHealth environment image](https://github.com/jupyterhealth/singleuser-image), which has Python, the JupyterHealth client, Jupyter AI, and common data science libraries pre-installed.

**Packages you install with `pip` will not persist across sessions!** If you must `pip install`, lut `%pip install ...` at the top of notebooks that need extra packages.

## Storage

Your home directory persists between sessions.
Add and edit whatever files you like, but try to keep file size down.

## Stop your session

When you're done, choose {menuselection}`File --> Hub Control Panel --> Stop My Server` so your server stops using cloud resources.

If you leave your hub session idle for long enough, it will be shut down automatically.

## Get help

- Problems with the hub itself (login loops, server won't start): use the [2i2c support process](xref:2i2c#support).
- Questions about JupyterHealth data or the exchange: ask in the [JupyterHealth Zulip channel](https://jupyter.zulipchat.com/#narrow/channel/jupyterhealth).
