perguntas--------------------------resposta
overflow:hidden;// para esconder o scrollbar

como fazer aniamcoes --------------
element{
	animation: name animation-duration;
	animation-delay:; //tempo de desenrolo da animacao
}
@keyfreames nome{
	from{
	}	
	to{
	}
		}

tambem pode ser definido em percentagem:

@keyfreames nome{
	0%{
	}	
	14%{
	}
	22%{
	}
	100%{
	}
		}
----------------------------------
para animacoes que se repetem PODEM REAGRUPA-LAS:

@keyfreames nome{
	0%, 75% , 100%, {
	}	
	14%{
	}
	22%{
	}
	88%, 97%{
	}
		}

animation-fill-mode: backwards;// pra começa com o efito definido no from 
ou
animation-fill-mode: forewards;// o efeito permanece apos a animacao


animation-timing-function: ease; // // a animacao se faz doucement
			 : ease-in;// a animacao começa doucement
			 : ease-out//a animacao termina doucement
			 : ease-in-out
			 : steps(5)// realisa a animacao em 5 passos dando pequenas pusas
			 : cubic-bezier()// para definir a os saltos temporais que quizer	
substitui o animation-delay de certa forma

animation: nono 500ms linear// o linear faz com a tempo de animacao seja fluido sem pausas ou atrasos

para parar uma animacao usa-se paused (animation-play-state: paused;)
animation: nono 500ms, fade paused; //aqui a animacao nono funciona mas a animacao fade fica parada 

animation-iteration-count: 3; // repete a animacao 3 vezes 
			 : infinite; // repete a animacao infinitas vezes 

animation-direction: reverse// rola a animacao no sentido contrario( do to para from)
		   : 
forma abrevida 
animation: name | duration | timing-function | delay | iteration-count | direction | fill-mode | play-state.
			 
