# Rakefile - Commandes utiles pour le projet

desc "Lancer le serveur Jekyll avec live reload"
task :serve do
  sh "bundle exec jekyll serve --livereload"
end

desc "Lancer le serveur Jekyll sans live reload"
task :build do
  sh "bundle exec jekyll build"
end

desc "Nettoyer les fichiers générés"
task :clean do
  sh "bundle exec jekyll clean"
end

desc "Afficher toutes les commandes disponibles"
task :help do
  puts "\nCommandes disponibles:\n"
  puts "  rake serve   - Lancer le serveur de développement avec hot reload"
  puts "  rake build   - Compiler le site statique"
  puts "  rake clean   - Supprimer les fichiers générés"
  puts "  rake help    - Afficher cette aide\n\n"
end
