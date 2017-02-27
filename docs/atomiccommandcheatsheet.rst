Atomic Command Cheat Sheet
==========================

This chapter contains cheat sheet for atomic commands

**The atomic command ``/usr/bin/atomic`` defines the entrypoint of Project Atomic hosts**


- ``atomic host`` host subcommands:
    - ``atomic host deploy <revision>`` deploys a specific commit.
    - ``atomic host install`` installs a layered rpm package.
    - ``atomic host rebase <refspec>`` downloads and deploys a new origin refspec.
    - ``atomic host rollback`` rollbacks to the previous version.
    - ``atomic host status`` shows the current status of the installed atomic host.
    - ``atomic host uninstall`` removes a layered rpm package.
    - ``atomic host unlock`` makes the current deployment mutable.
    - ``atomic host upgrade`` upgrades to a newer version.
- ``atomic containers`` container subcommands:
    - ``atomic containers delete <name>`` deletes specified container.
    - ``atomic containers list`` lists the installed containers.
    - ``atomic containers trim`` discards unused blocks on running containers.
    - ``atomic containers update <name>`` updates a container.
    - ``atomic containers rollback <name>`` rolls back a container to a previous version (only for system containers).
- ``atomic diff`` shows difference between to container images, RPMs or file diff.
- ``atomic images`` image subcommands:
    - ``atomic images delete <name>`` marks an image for deletion.
    - ``atomic images generate`` generates missing image manifests.
    - ``atomic images info <name>`` returns LABEL Information of the image.
    - ``atomic images list`` displays all the container image present on the host.
    - ``atomic images prune`` deletes dangling images.
    - ``atomic images update <name>`` pulls latest image from registry.
    - ``atomic images verify <name>`` verifies that the image is updated.
    - ``atomic images version <name>`` displays image 'Name Version Release' label.
- ``atomic install <name>`` executes container image install method.
- ``atomic mount`` mounts container image to a specific directory.
- ``atomic pull`` pulls the latest image from the repository.
- ``atomic push (upload)`` pushes (upload) the latest image to the repository.
- ``atomic run <name>`` executes container image run method.
- ``atomic scan <name>`` scans the image or container.
- ``atomic sign <name>`` signs the specified image.
- ``atomic stop <name>`` executes container image stop method.
- ``atomic storage (migrate)`` manages container storage.
- ``atomic top`` shows stats about processes running inside container.
- ``atomic trust`` manages container trust policy.
- ``atomic uninstall <name>`` uninstalls the container from the atomic host.
- ``atomic unmount`` unmounts container image.

We have blog post for few commands. Check `this <https://trishnag.wordpress.com/2016/08/11/getting-started-with-atomic-commands/>`_.
