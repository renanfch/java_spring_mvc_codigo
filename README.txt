Testado com JRE8 e JRE9, Apache Tomcat 7,8,9

1) Para compilar e empacotar na linha de comando use:

> mvn clean package

2) Para rodar no Eclipse com Tomcat no profile "dev" adicione "-Dspring.profiles.active=dev" 
nas "Run Configurations..." (ou descomento o método "onStartup" na classe "ServletSpringMVC")

Ao rodar pelo Eclipse e Tomcat acesse 

http://localhost:8080/casadocodigo

3) Para rodar na linha de comando (no profile dev usando tomcat 9) use:

> java -jar -Dspring.profiles.active=dev target/dependency/webapp-runner.jar target/*.war

e acesse http://localhost:8080/

Tags de aprendizado:
@Autowired
@Bean,
@EnableWebMvc,
@ComponentScan,
@EnableCaching,
@EnableTransactionManagement,
@Profile,
@EnableWebSecurity,
@Controller,
@ControllerAdvice ( Controller que intercepta os outros )
@RequestMapping(value="/login", method=RequestMethod.GET)
@Scope(value=WebApplicationContext.SCOPE_REQUEST),
@ExceptionHandler(Exception.class)
@RequestMapping(method=RequestMethod.GET)
@Cacheable(value="produtosHome")
@AuthenticationPrincipal
@CacheEvict(value="produtosHome", allEntries=true)
@PathVariable("id")
@Repository
@Entity
@Component
@Embeddable
@Id @GeneratedValue(strategy=GenerationType.IDENTITY)
@ElementCollection
@OneToMany(fetch=FetchType.EAGER, cascade=CascadeType.PERSIST)

ModelAndView("redirect:/carrinho");
MailSender,
JavaMailSenderImpl,
Callable<>,
heroku, 
InternalResourceViewResolver,
CacheManager,
JsonViewResolver,
CharacterEncodingFilter


<%@ taglib uri="http://java.sun.com/jsp/jstl/core" prefix="c"%>
<%@ taglib uri="http://java.sun.com/jsp/jstl/fmt" prefix="fmt" %>
<%@ taglib uri="http://www.springframework.org/tags" prefix="s"%>
<%@ taglib uri="http://www.springframework.org/security/tags" prefix="security" %>
<%@ taglib tagdir="/WEB-INF/tags" prefix="tags"%>


