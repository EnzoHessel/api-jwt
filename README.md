###   a p i - j w t 

<h1>
  Rotas
</h1>
<p>
  /auth/login <br>
  /auth/register <br>
  /user
</p>
 
<span>falta configurar o cors</span

<p>
  <br><br><br>
import org.springframework.context.annotation.Configuration;<br>
import org.springframework.web.servlet.config.annotation.CorsRegistry;<br>
import org.springframework.web.servlet.config.annotation.WebMvcConfigurer;<br>

@Configuration<br>
public class CorsConfig implements WebMvcConfigurer {<br>

    @Override<br>
    public void addCorsMappings(CorsRegistry registry) {<br>
        registry.addMapping("/**")<br>
                .allowedOrigins("http://localhost:4200")<br>
                .allowedMethods("GET", "POST");<br>
    }<br>
}<br>
</p>
