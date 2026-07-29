# Assurance Forge Examples

Version-controlled example projects for
[Assurance Forge](https://github.com/lasrod/assurance-forge).

These projects serve two purposes:

- demonstrate complete Assurance Forge projects that can be opened directly;
- provide stable, named fixtures for manual feature and regression testing.

## Projects

| Project | Purpose |
| --- | --- |
| [`kitchen-blender`](projects/kitchen-blender/) | A substantial safety case covering a domestic kitchen blender. Useful for general navigation, layout, terminology, and SACM compatibility testing. |
| [`gsn-pattern-decorators`](projects/gsn-pattern-decorators/) | Focused GSN pattern-notation project with uninstantiated and combined undeveloped/uninstantiated goals. |

## Open a project

Clone this repository, then use **File → Open Project** in Assurance Forge and
select the project's `af.proj` file:

```text
projects/<project-name>/af.proj
```

When this repository is initialized as the Assurance Forge `examples`
submodule, the same projects are available at:

```text
examples/projects/<project-name>/af.proj
```

Examples are committed baselines. If a test edits or saves a project, restore it
before the next test:

```bash
git -C examples restore .
git -C examples clean -fd
```

## Contribution rules

- Keep each example self-contained beneath `projects/<project-name>/`.
- Document its purpose, expected behavior, and manual test procedure.
- Do not commit API keys, personal information, local session state, backups, or
  generated exports.
- Prefer small focused projects for feature tests and richer projects for
  end-to-end workflows.
- Validate SACM files and open the project in Assurance Forge before publishing.

The examples are licensed under the MIT License.
