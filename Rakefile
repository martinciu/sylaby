namespace :sylaby do

  desc "sylaby w kolejnosci"
  task :ordered do
    spolgloski = %w(b c ć d f g h k l ł m n ń p r s ś t w x z ż ź)
    samogloski = %w(a e i j o u y)
    sylaby = []
    spolgloski.each do |spolgloska_1|
      samogloski.each do |samogloska|
        spolgloski.each do |spolgloska_2|
          sylaby << "#{spolgloska_1}#{samogloska}#{spolgloska_2}"
        end
      end
    end
    File.open("sylaby.txt", 'w') {|f| f.write(sylaby.join(" ")) }
  end

end

task :default => ["sylaby:ordered"]
