.PHONY: clean sofle ferris

all: sofle ferris

sofle: ../config/sofle.keymap
	keymap -c ./kdrawer-cfg.yaml parse -z ../config/sofle.keymap >sofle.yaml
	keymap -c ./kdrawer-cfg.yaml draw sofle.yaml >sofle.svg

ferris:
	keymap -c ./kdrawer-cfg.yaml parse -z ../config/cradio.keymap >cradio.yaml
	keymap -c ./kdrawer-cfg.yaml draw cradio.yaml >cradio.svg

clean:
	rm sofle.yaml cradio.yaml
