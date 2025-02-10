## By default, the generator will use rdgen.crayoneater.org to generate your custom client installers. Follow these instructions to use your own github account to generate your custom client installers.

## To fully host the client generator yourself, you will need to following:

<ol>
    <li>A Github account with a fork of the rdgen <a href=https://github.com/bryangerlach/rdgen>rdgen</a>  </li>
    <li>A Github fine-grained access token with permissions for your rdgen repository  
        <ul>
            <li>login to your github account  </li>
            <li>click on your profile picture at the top right, click Settings  </li>
            <li>at the bottom of the left panel, click Developer Settings  </li>
            <li>click Personal access tokens  </li>
            <li>click Fine-grained tokens  </li>
            <li>click Generate new token  </li>
            <li>give a token name, change expiration to whatever you want  </li>
            <li>under Repository acces, select Only select repositories, then pick your rdgen repo  </li>
            <li>give Read and Write access to actions and workflows  </li>
        </ul>
    </li>
    <li>Setup environment variables / secrets:
        <ul>
            <li>environment variables on the server running rdgen:  
                <ul>
                <li>GHUSER="your github username"  </li>
                <li>GHBEARER="your fine-graned access token"  </li>
                </ul></li>
            <li>optional github secrets (setup on your github account for your rdgen repo):  
                <ul>
                <li>WINDOWS_PFX_BASE64  </li> 
                <li>WINDOWS_PFX_PASSWORD  </li> 
                <li>WINDOWS_PFX_SHA1_THUMBPRINT</li>  
                </ul></li> 
        </ul>
    </li>
</ol>