## Interfaces


Interfaces são métodos e atributos pré-estabelecidos utilzados como regra.

	interface Template {
		public function setVariable($name, $var);
		public function getHtml($template);
	}

	class Template implements Template {
		private $vars = array();

		public function setVariable($name, $var) {
			$this->vars[$name] = $var;
		}

		public function getHtml($template) {
			foreach($this-$vars as $name => $value) {
				$template = str_replace('{' . $name . '}', $value, $template);
			}
			return $template;
		}
	}

Interfaces estendíveis

	interface {
		public function foo();
	}

	interface b extends a {
		public function baz(Baz $baz);
	}

Herança multipla

	interface a {}
	interface b {}

	interface c extends a, b {}

	class d implements c {}

Interface com constantes

	interface a {
		const b = 'Interface constant'
	}

	echo a::b;