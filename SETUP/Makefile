export MakeInc_cmd=${SRCROOT}/makedefs/MakeInc.cmd
export MakeInc_def=${SRCROOT}/makedefs/MakeInc.def
export MakeInc_rule=${SRCROOT}/makedefs/MakeInc.rule
export MakeInc_dir=${SRCROOT}/makedefs/MakeInc.dir


include $(MakeInc_cmd)
include $(MakeInc_def)

SETUP_SUBDIRS = 	\
	config		\
	decomment	\
	setsegname	\
	md

UNAME_S := $(shell uname -s)
	ifeq ($(UNAME_S),Darwin)
		SETUP_SUBDIRS += kextsymboltool
	endif

include $(MakeInc_rule)
include $(MakeInc_dir)
