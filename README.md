# desafio-Class---DIO

class Heroi {
    constructor(nome,tipo) {
        this.nome = nome;
        this.tipo = tipo;
    }

    atacar() {
        let ataque;
        switch (this.tipo) {
            case 'mago':
                ataque = 'usou magia';
                break;
            case 'guerreiro':
                ataque = 'usou espada';
                break;
            case 'monge':
                ataque = 'usou artes marciais';
                break;
            case 'ninja':
                ataque = 'usou shuriken';
                break;
            default:
                ataque = 'usou um ataque desconhecido';
                break;
        }
        console.log(`O ${this.tipo} atacou usando ${ataque}`);
    }
}


const heroi1 = new Heroi('Arthur', 'guerreiro');
const heroi2 = new Heroi('Merlin', 'mago');
const heroi3 = new Heroi('Shifu', 'monge');
const heroi4 = new Heroi('Ryu', 'ninja');

heroi1.atacar();
heroi2.atacar();
heroi3.atacar(); 
heroi4.atacar(); 
