# ![OCCOperatorImage](./resources/OperatorIcon.png) OCP Console Customizer

![Static Badge](https://img.shields.io/badge/current_version-1.0.22-green)


operator-sdk init --plugins=ansible --domain dovid
operator-sdk create api --group ocp-console-customizer --version v1alpha1 --kind ConsoleCustomizer --generate-role
operator-sdk create api --group ocp-console-customizer --version v1alpha1 --kind ConsoleCustomizerSkin

Change Makefile, swipe docker for podman and fix IMAGE_TAG_BASE and IMG ?= $(IMAGE_TAG_BASE):$(VERSION)


make docker-build docker-push

make deploy


