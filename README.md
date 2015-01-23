# bootstrap-codeigniter
Helper para manejar bootstrap 3 en las vistas de codeigniter 

<h1> Example </h1>

<h3> Controller </h3>

	public function index()
	{	
		//load helper bootstrap
		$this->load->helper('bootstrap');
		//call view
		$this->load->view('yourview');		
	}

<h3> View </h3>
<br>

	echo form_open("lol/");
	$atributos = array('style' 	=> 'text-align: center;');
	echo form_input_text('nombre', 'Ingresa nombre', $atributos);
	echo form_input_password('password','Ingresa contraseña', $atributos);
	echo form_input_checkbox('remember','Recordar');
	echo form_input_radio('area','Valor 1', 'valor1');
	echo form_input_radio('area','Valor 2', 'valor2');
	echo form_input_radio('area','Valor 3', 'valor3');
	echo form_input_textarea('area','ingresa una descripcion');
	echo form_input_select("lol");
	$options = array('1' => 1,'2' => 2);
	echo select_options($options);
	echo form_submit("Enviar formulario");
	echo form_close();


