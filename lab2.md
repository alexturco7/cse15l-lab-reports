`import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    String output = "";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/add-message")) {
            String[] parameters = url.getQuery().split("=");
            output += parameters[1] + "\n";
        }
        return output;
    }
}

public class StringServer {
    public static void main(String[] args) throws IOException {
        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}`
