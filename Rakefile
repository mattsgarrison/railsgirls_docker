desc "Connect to Docker image's shell. Provide image name you want to connect to."
task :shell, :name do |t, args|
  sh "sudo docker run -t -i #{args.name} /bin/bash"
end

desc "Build Docker image"
task :build, :tag do |t, args|

  sh "sudo docker build -t '#{args.tag}' ."

end
