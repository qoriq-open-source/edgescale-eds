#####################################
#
# Copyright 2017-2019 NXP
#
#####################################

INSTALL_DIR ?= /
INSTALL ?= install

all:
	go get github.com/joho/godotenv
	go build --ldflags="-s -w" -o es-watchdog

clean:
	rm es-watchdog

install:
	$(INSTALL) -d --mode 755 $(INSTALL_DIR)/usr/local/edgescale/bin
	sudo cp -r es-watchdog $(INSTALL_DIR)/usr/local/edgescale/bin

