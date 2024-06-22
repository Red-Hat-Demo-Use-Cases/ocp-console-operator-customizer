operator-sdk init --plugins=ansible --domain dovid
operator-sdk create api --group ocp-console-customizer --version v1alpha1 --kind ConsoleCustomizer --generate-role
operator-sdk create api --group ocp-console-customizer --version v1alpha1 --kind ConsoleCustomizerSkin --generate-role

Change Makefile, swipe docker for podman and fix IMAGE_TAG_BASE and IMG ?= $(IMAGE_TAG_BASE):$(VERSION)


make docker-build docker-push

make deploy