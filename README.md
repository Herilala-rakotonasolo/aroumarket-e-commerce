<p>Cette Application est pour une site de Commerce</p>
<h3>##Installation</h3>
Ouvrer votre ligne de commande :
<p>1- Clounez l'application</p>

<p>2-Installer toutes les dependances :</p>
ouvrez votre terminal et tapez
<ul>
    <li><span style="color :'red'"> composer -install</span> puis npm install & npm run dev</li>
</ul>
<p>3-Ajoutez cette ligne de code dans : vendor\laravel\ui\auth-backend\AuthenticatesUsers.php</p>

    protected function authenticated(Request $request, $user)
    {
        if($user->admin){
            return  redirect(route('admin'));
        }
    }
