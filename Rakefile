task :default => [:proof_readme]

task :proof_readme do
  require 'html/proofer'

  Dir.mkdir("proof") unless File.exists?("proof")
  system "cp *.html proof/"
  HTML::Proofer.new("./proof").run
end
