#!/bin/bash

serve: build
	ZOLA_ROOT=. source z-dev-scripts/static-watcher.sh; watch_static & zola serve -O
build:
	ZOLA_ROOT=. source z-dev-scripts/static-watcher.sh; build && \
	zola build
