# nix-flake-poetry-example


## Development

To drop into a shell:

	nix develop
	
To run a python file quick:

	nix develop -c python src/nix_flake_poetry_example/__init__.py
	
Launch this repo in vs code with the path set correctly:

	nix develop -c code .
	
Format python files:

	nix develop -c black .
	
Format nix files:

	nix develop -c nixpkgs-fmt .
	
## Building

To build the package:

	nix build

Results will be placed in `./result`. Run a wrapper script with:

	./result/bin/nix-flake-poetry-example
