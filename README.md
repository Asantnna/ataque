# ataque
class Heroi {
  constructor(nome, idade, tipo) {
    this.nome = nome;
    this.idade = idade;
    this.tipo = tipo;
  }

  atacar() {
    const ataque = this.tipo === "mago" ? "magia" :
      this.tipo === "guerreiro" ? "espada" :
      this.tipo === "monge" ? "artes marciais" :
      "shuriken";

    console.log(`O ${this.tipo} atacou usando ${ataque}`);
  }
}

const mago = new Heroi("Merlin", 1000, "mago");
const guerreiro = new Heroi("Arthur", 500, "guerreiro");
const monge = new Heroi("Bruce Lee", 80, "monge");
const ninja = new Heroi("Rin", 20, "ninja");

mago.atacar();
guerreiro.atacar();
monge.atacar();
ninja.atacar();
