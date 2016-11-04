# EmbeddedResource
This library loads .dll`s from embedded resources of your project. This code is not mine

.dll has to be added to your project as embedded resource
and you have to add link for this .dll to links and in propeties of this lib you should change local copy from true to false

example of usage:

	    try
            {
                string resource1 = "YourApp.Microsoft.Expression.Interactions.dll";
                string resource2 = "YourApp.System.Windows.Interactivity.dll";
                EmbeddedAssembly.Load(resource1, "Microsoft.Expression.Interactions.dll");
                EmbeddedAssembly.Load(resource2, "System.Windows.Interactivity.dll");
            }
            catch { }
