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
import org.springframework.context.annotation.Configuration;
import org.springframework.web.servlet.config.annotation.CorsRegistry;
import org.springframework.web.servlet.config.annotation.WebMvcConfigurer;

@Configuration
public class CorsConfig implements WebMvcConfigurer {

    @Override
    public void addCorsMappings(CorsRegistry registry) {
        registry.addMapping("/**")
                .allowedOrigins("http://localhost:4200")
                .allowedMethods("GET", "POST");
    }
}
</p>
