desc 'Test strings files'
task :test do
  Dir.foreach('.') do |path|
    next unless path =~ /\.lproj$/
    system "plutil -lint #{path}/Localizable.strings"
    puts
  end
end

task :default => :test
