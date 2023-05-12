package com.aulaandroid.frasesmotivacionais;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import java.util.Random;
import android.widget.Button;
import android.view.View.OnClickListener;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {
    /**
     * Atribuição dos elementos do Desgin da MainActivity
     */
    private TextView frases;
    private Button gerarFrases;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main); //Inicialização da MainActivity

        frases = findViewById (R.id.frases); //Encontrando a variável frases pelo ID
        gerarFrases = findViewById(R.id.gerarFrases); //Encontrando a variável gerarFrases pelo ID

        getSupportActionBar ().hide(); //Esconder Action Bar

        gerarFrases.setOnClickListener(new View.OnClickListener(){
            @Override
            /**
             * Com o uso do onClick no botão 'gerarFrases' do Design, assim que o botão seja selecionado uma da 10 frases apareceram de forma aleatorizada
             * Utilizando o RANDOM.
             */
            public void onClick(View v){
                String[] frasesMotivacionais = {"Que os dias bons se tornem rotina e os ruins se tornem raros.",
                        "A felicidade não é algo pronto. Ela é feita das suas próprias ações.",
                        "Tentar é a única maneira de saber se vai dar certo.", "Você pode, se acreditar que pode",
                        "A influência das boas pessoas ninguém consegue apagar.", "Se não puder fazer tudo, faça tudo que puder.",
                        "Até o maior dos prédios começa no chão.", "O segredo é um só: acreditar que tudo vai dar certo, porque vai.",
                        "O otimismo é o imã da felicidade.", "Que os dias ruins se tornem raros e os bons virem rotina."};
                int sorteio = new Random().nextInt(10);
                frases.setText(frasesMotivacionais[sorteio]); // Mostrando ao usuário a frase aleatorizada

            }
        });
    }
}
