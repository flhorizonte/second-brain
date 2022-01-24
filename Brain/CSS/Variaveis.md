### Variaveis

Basic Usage

	element {
			--cor-bg-principal: brown;
	}

	foo {
			background-color: var(--cor-bg-principal);
	}

How var() Works

- CSS variables can have a global or local scope.
- Global variables can be acessed  through the entire document, while local variables can be used only inside the selector where it is declared.
- To createw a variable with global scope, declare it inside the `:root` selector.
		`
				:root {
					--blue: #1e90ff;
					--white: #ffffff;
				}
		`
- To create a variable with local scope, declare it inside the selector that is going to use it.