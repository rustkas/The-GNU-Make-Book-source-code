env_file = /tmp/env
env_shell = $(shell rm -f $(env_file))$(foreach V,$1,$(shell echo export $V=$($V) >> $(env_file)))$(shell echo '$2' >> $(env_file))$(shell /bin/bash -e $(env_file))

export FOO=bar

$(info  $(call env_shell,FOO,printenv | grep FOO))
all: ; @printenv | grep FOO