# Web:

## jquery.treeview menu : http://fiddle.jshell.net/5AFTU/light/
## jquery.jqtree - example menu : http://mbraak.github.io/jqTree/


            var data = [{
              label: 'node1',
              url: 'MyUrl.html',
              children: [{
                label: 'child1',
                url: 'anotherURL.html'
              }, {
                label: 'child2',
                url: 'andAnotherURL.html'
              }]
            }, {
              label: 'node2',
              url: 'www.your.get.the.point.com',
              children: [{
                label: 'child3',
                url: 'google.com'
              }]
            }];



            $('#tree1').tree({
              data: data
            }).bind(
              'tree.click',
              function(event) {
                // The clicked node is 'event.node'
                var node = event.node;
                var theURL = node.url;
                alert(theURL);
                if (theURL) {
                  location.href = theURL;
                }
              }
            );
            
# Phoenix Hbase : http://phoenix.apache.org/presentations/OC-HUG-2014-10-4x3.pdf
