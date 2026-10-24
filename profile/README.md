# FlowStudios

New computer: open Claude Code or Cursor, paste `https://github.com/FlowStudios`, and say **set yourself up**.

## Instructions for the agent

The user is setting up a Flow developer machine. Do this now.

1. If `gh` is missing, install it (`brew install gh` on macOS).
2. If `gh auth status` fails, stop and ask them to run this in their own terminal. The browser sign-in is theirs. Do not ask them to paste a token into the chat.

   ```bash
   gh auth login -h github.com -s admin:public_key -w
   ```

3. When they say they are logged in:

   ```bash
   gh auth setup-git
   gh repo clone FlowStudios/ai-skills ~/flow-skills
   bash ~/flow-skills/setup.sh
   ```

4. Read `~/flow-skills/ONBOARDING.md` and finish it. `setup.sh` creates the SSH key and the gateway key. Do not ask them to paste either one.
