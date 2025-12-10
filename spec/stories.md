# STRUCTURE

- Requirements are written using the `As I, I want, So that` format. E.g.:

```
As an enrolled user,
I want to be able to change my display name,
So that I can personalize my profile.
```

- Do not include the acceptance criteria in the stories file. Acceptance criteria are maintained by the test agent in their own file.

- Stories are in written in yaml following this format:

```yaml
story:
  - Id: story-001
    priority: unprioritized
    title: Allow users to change their display name
    who: As an enrolled user
    what: I want to be able to change my display name
    why: So that I can personalize my profile
```

- The priority field must be set to `unprioritized` when first created.
- Prioritiztation is a separate workflow after the story is created.

 # STORIES

All stories are maintained in yaml in the following file:

@./spec/stories.yaml
